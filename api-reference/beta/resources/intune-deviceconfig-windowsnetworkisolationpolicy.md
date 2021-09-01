---
title: тип ресурса windowsNetworkIsolationPolicy
description: Windows Политика изоляции сети
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c93d9292df647ccec7f6047cbb7a922329855f4e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790390"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>тип ресурса windowsNetworkIsolationPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Политика изоляции сети

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enterpriseNetworkDomainNames|Коллекция String|Это список доменов, входящих в границы предприятия. Данные из одного из этих доменов, которые отправляются на устройство, будут считаться корпоративными данными и защищены. Эти расположения будут считаться безопасным пунктом назначения для общих корпоративных данных.|
|enterpriseCloudResources|Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Содержит список корпоративных доменов ресурсов, которые размещены в облаке, которые необходимо защитить. Подключения к этим ресурсам считаются корпоративными данными. Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80). Прокси-сервер, используемый для этой цели, также должен быть настроен с помощью политики EnterpriseInternalProxyServers. Эта коллекция может содержать не более 500 элементов.|
|enterpriseIPRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети. Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются. Эти расположения будут считаться безопасным пунктом назначения для общих корпоративных данных. Эта коллекция может содержать не более 500 элементов.|
|enterpriseInternalProxyServers|Коллекция String|Это список внутренних прокси-серверов, разделенных запятыми (например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"). Эти прокси-серверы настроены администратором для подключения к определенным ресурсам в Интернете. Они считаются корпоративными расположениями в сети. Прокси-ресурсы используют только в настройке политики EnterpriseCloudResources для принудительного трафика на указанные облачные ресурсы через эти прокси.|
|enterpriseIPRangesAreAuthoritative|Boolean|Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей. Значение по умолчанию: false.|
|enterpriseProxyServers|Коллекция String|Это список прокси-серверов. Любой сервер, не в этом списке, считается непредприятным.|
|enterpriseProxyServersAreAuthoritative|Boolean|Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы. Значение по умолчанию: false.|
|neutralDomainResources|Коллекция String|Список доменных имен, которые можно использовать для работы или личного ресурса.|

## <a name="relationships"></a>Связи
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
      "@odata.type": "microsoft.graph.ipRange"
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



