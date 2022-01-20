---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: abf6f2398b8f2b4ac96c0d8c9e0a3c7b718c6331
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135225"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel."
    DisplayName = "Inferring User Intent through browsing behaviors"
    IsPending = $true
    Number = "USPTO-3954432633"
    WebUrl = "https://patents.gov/3954432633"
}

New-MgUserProfilePatent -UserId $userId -BodyParameter $params

```