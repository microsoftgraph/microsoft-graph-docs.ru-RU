---
title: Тип ресурса informationalUrl
description: Сведения о базовой профиля приложения.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816984"
---
# <a name="informationalurl-resource-type"></a>Тип ресурса informationalUrl

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сведения о базовой профиля приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|маркетинг|Строка| Ссылка на приложение маркетинговых страницы. Например, https://www.contoso.com/app/marketing |
|конфиденциальность|Строка| Ссылка на заявление о конфиденциальности приложения. Например, https://www.contoso.com/app/privacy |
|Поддержка|Строка| Ссылка на страницу поддержки приложения. Например, https://www.contoso.com/app/support |
|termsOfService|Строка| Ссылка на условия приложения службы оператора. Например, https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
