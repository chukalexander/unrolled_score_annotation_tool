# Custom annotation tool to create data for Music Information Retrieval

- Annotates unrolled sheet music (.png) by storying xy-coordinates of noteheads, systems and barlines.
- Stores said coordinates into .npy arrays
- Data can be for Optical Music Recognition(OMR) or Score Following

### Sample

- Raw .png of unannotated score
- 
![image](https://github.com/chukalexander/unrolled_score_annotation_tool/assets/117527004/3558d093-152a-4703-a78b-178ea72c04f0)


- Annotated score
- 
![image](https://github.com/chukalexander/unrolled_score_annotation_tool/assets/117527004/f8d3bdf3-516b-4144-bef3-e0457cfab635)


### Instruction

### 1. Sample
- test Sample section which will load and display above samples

### 2. Change directory
- Change directory 'data_dir' to raw dataset which needs to be annotated
- Change 'song' to file name of .png of unrolled sheet music

### 3. NOTES
- Uncomment "np.save(notes_dir, note_ary)"
- Click the noteheads in decending pitch order from the first to last beat.
- 1st Key press to save
- 2nd Key press to close window

### 4. SYSTEM
- Uncomment "np.save(sys_dir, sys_ary)"
- Click the top left, bottom left, top right, bottom right corners of the system in order
- 1st Key press to save
- 2nd Key press to close window

### 5. BARS
- Uncomment np.save(bar_dir, bar_ary)
- Start from the barline connecting bar 1 and 2
- Click top of barline, then bottom of barline
- Continue onto next bar
- 1st Key press to save
- 2nd Key press to close window

### Dataset created
