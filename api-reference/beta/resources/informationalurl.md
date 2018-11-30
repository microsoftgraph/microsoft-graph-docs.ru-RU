---
title: Тип ресурса informationalUrl
description: Сведения о базовой профиля приложения.
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079866"
---
# <a name="informationalurl-resource-type"></a>Тип ресурса informationalUrl

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сведения о базовой профиля приложения.

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------------|:--------|:----------|
|маркетинг|String| Ссылка на приложение маркетинговых страницы. Например, https://www.contoso.com/app/marketing |
|конфиденциальность|String| Ссылка на заявление о конфиденциальности приложения. Например, https://www.contoso.com/app/privacy |
|Поддержка|String| Ссылка на страницу поддержки приложения. Например, https://www.contoso.com/app/support |
|termsOfService|String| Ссылка на условия приложения службы оператора. Например, https://www.contoso.com/app/termsofservice |

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