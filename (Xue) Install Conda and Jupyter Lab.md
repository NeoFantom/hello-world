Download Miniconda
===

Open url: [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)

Download your version. Install with default configurations

Get conda ready
===

* For Windows only: Open app "**Anaconda powershell prompt**", input this command, press enter.
  * `conda init powershell`
* For Windows only: Open **terminal** (called "terminal" on MacOS or "powershell" on Windows), **try** execute
  * `conda`
  * On failure: Allow powershell to execute conda's launching script. Reopen powershell in Administrator mode and execute command
    * `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned`
    * Close all powershell windows.
  * On success (you see conda's help information): Go on.
* Create a new virtual environment by
  * `conda create -n [name]` (Notice: change `[name]` to your favorite name and remove `[]`, the same below)
* Activate the environment you just created by
  * `conda activate [name]`
* Install necessary packages by (Notice: Conda will download anything required by these packages, such as Python, automatically)
  * `conda install jupyterlab numpy matplotlib tqdm`
* Add a channel so that we can access qutip package.
  * `conda config --append channels conda-forge`
* Install qutip
  * `conda install qutip`

Begin programming
===

* Create an empty directory for programming.
* Copy it's path.

> Every time you want to write python in *Jupyter Lab*, open terminal (or powershell for Windows) and do the following.

* Change current directory.
  * **Remember this!!!**
  * First way:
    * `cd [path]` (Change `[path]` to copied path)
  * Second way (equivalent):
    * In the folder, right-click and select "Open in terminal/powershell"
* Use `ls` to check that it's empty.
* Open Jupyter Lab by
  * `jupyter lab`
* Note: If you want to install another package in conda, make sure to close Jupyter Lab in both terminal and browser, install, and then reopen Jupyter Lab again.

In your browser (automatically open by Jupyter Lab)

* Create a new notebook.
* Save and rename the notebook.
* Begin coding!
