---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e2419170c99c68ab2d454c6bf8a305a5de70fc29
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224815"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    RedundancyDetection = @{
        IsEnabled = $false
        SimilarityThreshold = 70
        MinWords = 12
        MaxWords = 400000
    }
    TopicModeling = @{
        IsEnabled = $false
        IgnoreNumbers = $false
        TopicCount = 50
        DynamicallyAdjustTopicCount = $false
    }
    Ocr = @{
        IsEnabled = $true
        MaxImageSize = 12000
    }
}

Update-MgComplianceEdiscoveryCaseSetting -CaseId $caseId -BodyParameter $params

```