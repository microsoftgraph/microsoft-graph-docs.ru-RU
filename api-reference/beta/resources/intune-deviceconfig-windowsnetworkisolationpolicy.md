---
title: Тип ресурса Виндовснетворкисолатионполици
description: Политика сетевой изоляции Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 515d1b89631b33907aef0ef19bbc3f28181dc5d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370769"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>Тип ресурса Виндовснетворкисолатионполици

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика сетевой изоляции Windows

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enterpriseNetworkDomainNames|Коллекция строк|Это список доменов, входящих в границы предприятия. Данные из одного из этих доменов, отправляемых на устройство, будут считаться корпоративными данными и защищены. Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным.|
|Вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection|Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Содержит список корпоративных доменов ресурсов, размещенных в облаке и требующих защиты. Подключения к этим ресурсам считаются корпоративными данными. Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80). Прокси-сервер, используемый для этой цели, также должен быть настроен с использованием политики Ентерприсеинтерналпроксисерверс. Эта коллекция может содержать не более 500 элементов.|
|enterpriseIPRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети. Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются. Эти расположения будут считаться безопасным пунктом назначения для предоставления общего доступа к корпоративным данным. Эта коллекция может содержать не более 500 элементов.|
|enterpriseInternalProxyServers|Коллекция строк|Это список внутренних прокси-серверов, разделенных запятыми (например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"). Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете. Они считаются корпоративными расположениями в сети. Прокси-серверы используются только в настройке политики вместо enterprisecloudresourceswindowsnetworkisolationcloudresourcecollection для принудительного передачи трафика в соответствующие облачные ресурсы через эти прокси-серверы.|
|enterpriseIPRangesAreAuthoritative|Boolean|Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей. Значение по умолчанию — false.|
|enterpriseProxyServers|Коллекция строк|Это список прокси-серверов. Любой сервер, не включенный в этот список, считается не предприятием.|
|enterpriseProxyServersAreAuthoritative|Boolean|Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы. Значение по умолчанию: false.|
|neutralDomainResources|Коллекция строк|Список доменных имен, которые могут использоваться для рабочего или личного ресурса.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```



