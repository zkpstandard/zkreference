%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%% Notes since 2019-04-01, Luís Brandão:
  % This LaTeX project is open for collaboration under the ZKProof.org terms.
  % The main file for compilation is zkproof-docs.tex (use pdfLaTeX)
  %%%%%%%%%%%%
  % SUMMARY:
  % The initial LaTeX version (2019-04-01) is a porting to LaTeX of the ZKProofs 
  %   docs downloaded from https://zkproof.org/documents.html in March 2019.
  % The porting included editorial adjustments for indexation, consistency, etc.
  % The underlying content was authored by the ZKProof team/collaborators.
  %%%%%%%%%%%%
  % VIEWING POPUP ANNOTATIONS:
    % Note: the popup annotations are not shown in the "Built-In" Overleaf PDF-viewer.
    % Option 1: Menu --> PDF viewer --> Native
    % Option 2: open the PDF file with a regular PDF-viewer in your local computer.
  %%%%%%%%%%%% 
  % ADDING COMMENTS AS POPUP ANNOTATIONS: 
  % To insert a blue popup, starting with "Your name\\Suggestion: " 
    % \suggest[your name]{your suggestion} 
  % To insert a green popup, starting with "Your name\\Edited: "
    % \edited[your name]{notes about what you edited} 
  % To insert a red popup, starting with "Your name\\To-do: "
    % \smttodo[your name]{note on something to be edited} 
  % To insert a blue popup starting with "Your name\\"
    % \popupColor{your name}{your comment}
  % If adding many popups, define shortcut commands in the end of ...-b-cmds.tex
    % This facilitates a selective search, highlight or omission of those comments
  %%%%%%%%%%%%
  % ADDING NEW CONTENT:
  % - New commands with global applicability: defined inside zkproof-docs-00-b-cmds.tex
  % - New non-appendix chapter: create a file name zkproof-docs-0<d>-....tex, where <d> is a digit
  % - New appendix chapter: use a file name zkproof-0<L>-<tttt>.tex, where <L> is a letter B, C, ...
  % - New content in the preamble: fit into existing file or create file with name zkproof-docs-00-<L>...
  % - Loading of new packages: add \usepackage{...} inside zkproof-docs-00-a-pkgs.tex
  % - Files with externally-generated figures go inside the subfolder \figs
  % - New bibliographic reference: include a bibtex formatted entry inside one of the .bib files
  %%%%%%%%%%%%
  % LOCAL COMPILATION:
  % - compile with pdfLaTeX (will later also make compatible with LuaLaTeX)
  % - the bibliography is using biblatex and biber
  % - check that 'biber' is set as the processor working with biblatex
  % To hide the popup annotations, add to the bottom of ...-b-cmds.tex:
    % \renewcommand{\popupColor}[3][]{}