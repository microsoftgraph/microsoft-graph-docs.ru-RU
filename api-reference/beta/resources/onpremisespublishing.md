---
title: Тип ресурса Онпремисеспублишинг
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: db81ef2c61142edb0d3ca58a67b34c7da34e71f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522216"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса Онпремисеспублишинг

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект **онпремисеспублишинг** представляет набор свойств для публикации локального [приложения](application.md).

## <a name="properties"></a>Свойства

| Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|кустомдомаинцертификате|String|Сведения о сертификате, связанном с приложением при использовании настраиваемого домена. NULL при использовании домена по умолчанию.|
|екстерналаусентикатионтипе|String|Detailed: параметры предварительной проверки подлинности для возможных значений `passthru`приложения `aadPreAuthentication`:,.|
|externalUrl|String|Опубликованный внешний URL-адрес приложения. Напримерhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|Внутренний URL-адрес приложения. Напримерhttps://intranet/ |
|исонпремпублишинженаблед|Логический|Указывает, выполняется ли публикация приложения в данный момент.|
|аппликатионсервертимеаут|String|Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения. Возможные значения: `default`, `long`. Используйте `long` , если серверу требуется более 60-75 секунд для ответа на запросы. Кроме того `long` , попробуйте получить доступ к приложению и состояние ошибки "внутренний тайм-аут".|
|истранслатехоссеадеренаблед|Логический|Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа. Сюда входит настройка правильного сайта для файлов cookie.|

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
2019-02-04 14:57:30 UTC -->
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
