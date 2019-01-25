---
title: Тип ресурса educationSynchronizationDataProvider
description: 'Представляет схему SIS источника. Это позволяет системы, чтобы знать, как сопоставление входящих данных схемы Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515498"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>Тип ресурса educationSynchronizationDataProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет схему SIS источника. Это позволяет системы, чтобы знать, как сопоставление входящих данных схемы Azure Active Directory (Azure AD).

> **Примечание:** В данном сложном типе абстрактный. Обращайтесь к определенным типам поставщиков данных из списка.

## <a name="derived-types"></a>Производные типы
| Тип | Описание |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | Использовать с помощью CSV-файлов в качестве источника ввода. |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | Используется с PowerSchool в качестве источника ввода. |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | Использовать с использованием интерфейса API OneRoster в качестве источника ввода. |

## <a name="properties"></a>Свойства

С этого типа свойств не представлено.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
