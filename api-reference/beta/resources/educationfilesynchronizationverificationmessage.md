---
title: Тип ресурса educationFileSynchronizationVerificationMessage
description: Представляет ошибки, возвращенной клиенту в ответ на запрос на запуск синхронизации профилей на основе CSV школа данных. Этот ресурс будет содержать ошибки, которые возникают из проверки. Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).
author: mmast-msft
ms.openlocfilehash: f2826f779aac3ba41146b6677f3d1e0364be92a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336066"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>Тип ресурса educationFileSynchronizationVerificationMessage

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ошибки, возвращенной клиенту в ответ на запрос на [Запуск синхронизации](../api/educationsynchronizationprofile-start.md) профилей на основе CSV школа данных. Этот ресурс будет содержать ошибки, которые возникают из проверки. Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **type** | string | Тип сообщения. Возможные значения: `error`, `warning`, `information`. | 
| **Имя файла** | string | Исходный файл, который содержит ошибки. |
| **description** | строка | Подробные сведения о типе сообщения. |

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