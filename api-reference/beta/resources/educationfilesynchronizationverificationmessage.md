---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e82ede1df5c17b99fdc40857fd97f1f90012711
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434979"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>Тип ресурса Едукатионфилесинчронизатионверификатионмессаже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| type        | string | Тип сообщения. Возможные значения: `error`, `warning`, `information`. |
| задан    | Строка | Исходный файл, который содержит ошибку.                                         |
| description | string | Подробные сведения о типе сообщения.                                 |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
  "type": "String",
  "fileName": "String",
  "description": "String"
}
```
