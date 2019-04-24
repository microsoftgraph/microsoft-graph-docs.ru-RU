---
title: Тип ресурса Едукатионсинчронизатиондатапровидер
description: 'Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507046"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Тип ресурса Едукатионсинчронизатиондатапровидер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет исходную схему SIS. Это позволяет системе узнать, как сопоставить входящие данные с схемой Azure Active Directory (Azure AD).

> **Примечание:** Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов поставщиков данных.

## <a name="derived-types"></a>ПроизВодные типы
| Тип | Описание |
|:-|:-|:-|
| [едукатионксвдатапровидер](educationcsvdataprovider.md) | Используется с CSV-файлами в качестве источника входных данных. |
| [едукатионповерсчулдатапровидер](educationpowerschooldataprovider.md) | Используется с PowerSchool в качестве источника входных данных. |
| [едукатиононеростерапидатапровидер](educationonerosterapidataprovider.md) | Используется с API OneRoster в качестве источника входных данных. |

## <a name="properties"></a>Свойства

Этот тип не представляет свойства.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
