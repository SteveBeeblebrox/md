# (c) Trin Wasinger 2021-2026
# Load using exec(__import__('requests').get('https://raw.githubusercontent.com/SteveBeeblebrox/md/refs/heads/main/md').text)
@lambda _:_()
def md():
  import IPython
  with open('README.md', 'w') as file:
    file.write('')
  @IPython.core.magic.register_line_cell_magic
  def md(line: str, cell: str | None = None):
      if cell: line += f'\n{cell}'
      with open('README.md', 'a') as file:
          file.write(line + '\n')
      display(IPython.display.Markdown(line));
del md;
