---
title: Тип ресурса onPremisesPublishing
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508183"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса onPremisesPublishing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Сведения о сертификате, связанных с приложением, при использовании настраиваемого домена. Использование домена по умолчанию значение NULL.|
|externalAuthenticationType|String|Дополнительные сведения об значение предварительной проверки подлинности для приложения возможными значениями являются: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|Опубликованные внешний URL-адрес для приложения. Пример:  |
|internalUrl|String|Внутренний URL-адрес приложения. Пример: |
|isOnPremPublishingEnabled|Логическое|Указывает, если приложение публикуется в настоящее время или нет.|
|applicationServerTimeout|String|Во время выполнения соединитель будет ожидать ответа из базы данных приложения до закрытия подключения. Возможные значения: `default`, `long`. Использование `long` Если сервер принимает более 60 75 секунд отвечать на запросы. Также попробуйте `long` Если вы не можете получить доступ к приложению и состояние ошибки «Время ожидания базы данных».|
|isTranslateHostHeaderEnabled|Логическое|Указывает, если приложение следует перевести URL-адреса в заголовке ответа. Этот компонент включает Установка правильное веб-узла для файлов cookie.|

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
