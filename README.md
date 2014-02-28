# bframe c library

## Overview:

## Using:

### Building and installing:

### Example

```C
#include <bframe.h>

int
main(int argc, char **argv)
{
  char data[] = "this is a message";
  bframe_t *bframe = new_bframe(data, strlen(data));

  int size;
  char *char_bframe = bframe_to_char(bframe, &size);

  clean_bframe(bframe);
  free(bframe);

  int number_of_frames;

  bframe_buffer_t *bframe_buffer = new_bframe_buffer();
  bframe_t *bframes = parse_char_to_bframes(char_bframe, size, bframe_buffer, &number_of_frames);

  clean_bframe(&bframes[0]);
  free(bframes);

  clean_bframe_buffer(bframe_buffer);
  free(bframe_buffer);

  return 0;
}

```
