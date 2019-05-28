Will be documenting my findings from running [PSALM](https://github.com/vimeo/psalm) on various repositories here

- Levels range from 1 - 8, 1 displays more errors(Strictest) and 8 is most lennient with error reporting
- Analysis is only done on folders under the `<projectFiles>` `<projectFiles>` section i.e


  ` <projectFiles> `
  
        `<directory name="src" />`
        
        `<directory name="docs" />`
        
        `<directory name="design" />`
        
        `<directory name="tests" />`
        
        `<ignoreFiles>`
        
            `<directory name="vendor" />`
            
        `</ignoreFiles>`
        
   ` </projectFiles>`
 `
