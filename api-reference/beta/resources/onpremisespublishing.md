---
title: Тип ресурса Онпремисеспублишинг
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568869"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса Онпремисеспублишинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Кустомдомаинцертификате|String|Сведения о сертификате, связанном с приложением при использовании настраиваемого домена. NULL при использовании домена по умолчанию.|
|Екстерналаусентикатионтипе|String|Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.|
|externalUrl|String|Опубликованный внешний URL-адрес приложения. Напримерhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|Внутренний URL-адрес приложения. Напримерhttps://intranet/ |
|Исонпремпублишинженаблед|Boolean|Указывает, выполняется ли публикация приложения в данный момент.|
|Аппликатионсервертимеаут|String|Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения. Возможные значения: `default`, `long`. Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы. Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".|
|Истранслатехоссеадеренаблед|Boolean|Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа. Сюда входит настройка правильного сайта для файлов cookie.|

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
