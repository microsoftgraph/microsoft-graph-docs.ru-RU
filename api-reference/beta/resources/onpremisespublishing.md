---
title: Тип ресурса onPremisesPublishing
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842541"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса onPremisesPublishing

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customDomainCertificate|Строка|Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена. Использование домена по умолчанию значение NULL.|
|externalAuthenticationType|Строка|Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.|
|externalUrl|Строка|Опубликованные внешний URL-адрес для приложения. Напримерhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|Строка|Внутренний URL-адрес приложения. Напримерhttps://intranet/ |
|isOnPremPublishingEnabled|Логический|Указывает, если приложение публикуется в настоящее время или нет.|
|applicationServerTimeout|Строка|Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения. Возможные значения: `default`, `long`. Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы. Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».|
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
