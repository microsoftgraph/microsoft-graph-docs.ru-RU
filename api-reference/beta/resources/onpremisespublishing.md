---
title: Тип ресурса onPremisesPublishing
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078692"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса onPremisesPublishing

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена. Использование домена по умолчанию значение NULL.|
|externalAuthenticationType|String|Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|Опубликованные внешний URL-адрес для приложения. Напримерhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|Внутренний URL-адрес приложения. Напримерhttps://intranet/ |
|isOnPremPublishingEnabled|Логический|Указывает, если приложение публикуется в настоящее время или нет.|
|applicationServerTimeout|String|Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения. Возможные значения: `default`, `long`. Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы. Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».|
|isTranslateHostHeaderEnabled|Логический|Указывает, если приложение следует перевести URL-адреса в заголовке ответа. Этот компонент включает Установка правильное веб-узла для файлов cookie.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
