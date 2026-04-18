# Week 1: Evolution, Philosophy, and the Lab

## Monday: Linux Genealogy
- **Concept:** Linux is technically the **Kernel** (the engine); GNU provides the **Tools** (the dashboard/controls).
- **History:** Derived from Unix principles, but contains zero Unix code.
- **Task:** Verify kernel version.
  - Command: `uname -a`

## Tuesday: Distribution Families
| Family | Current Tool | Legacy Tool | Format | My VM |
| :--- | :--- | :--- | :--- | :--- |
| **Debian** | `apt` | `apt-get` | `.deb` | Debian 12 |
| **Red Hat** | `dnf` | `yum` | `.rpm` | Rocky 9 |

*Note: The LPI exam may use `yum` and `dnf` interchangeably. `dnf` is the modern successor.*

## Wednesday: Open Source Licensing
- **GPL (General Public License):** - Known as **"Copyleft"**. 
  - If you modify and distribute the code, you **must** share your changes under the same license.
- **Permissive (BSD/MIT):** - Allows you to modify code and keep it proprietary if desired.
- **FOSS:** Free and Open Source Software.

## Thursday: The Shell
- **Default Shell:** Bash (Bourne Again Shell).
- **Prompt Identification:**
  - `$` = Standard User (Limited permissions).
  - `#` = Root User (Full system administrative power).

## Friday: Cloud & Connectivity
- **IaaS:** Infrastructure as a Service (e.g., My Proxmox setup).
- **PaaS:** Platform as a Service (e.g., Heroku, Google App Engine).
- **SaaS:** Software as a Service (e.g., Gmail, Microsoft 365).
- **Connectivity:** `ping -c 3 google.com`
