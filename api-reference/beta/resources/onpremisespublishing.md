---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341805"
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
|Исонпремпублишинженаблед|Логический|Указывает, выполняется ли публикация приложения в данный момент.|
|Аппликатионсервертимеаут|String|Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения. Возможные значения: `default`, `long`. Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы. Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".|
|Истранслатехоссеадеренаблед|Логический|Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа. Сюда входит настройка правильного сайта для файлов cookie.|

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
  "suppressions": []
}
-->
