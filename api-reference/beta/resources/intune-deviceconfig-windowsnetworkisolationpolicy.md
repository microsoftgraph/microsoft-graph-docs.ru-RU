---
title: Тип ресурса windowsNetworkIsolationPolicy
description: Политики изоляции сети Windows
ms.openlocfilehash: 89c7db0453c76f6ec5016a4701bf357e27c579bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078283"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>Тип ресурса windowsNetworkIsolationPolicy

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политики изоляции сети Windows
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enterpriseNetworkDomainNames|Коллекция String|Это список доменов, входящих в границы предприятия. Данные из одного из этих доменов, которые отправлены на устройство будет считаться корпоративных данных и защищенные. Безопасные место назначения для корпоративных данных открыть общий доступ в будут считаться местоположениях.|
|enterpriseCloudResources|Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)|Содержит список доменов ресурсов предприятия, размещенные в облаке, должны быть защищены. Подключения к этим ресурсам считаются корпоративными данными. Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80). Для этой цели использовать прокси-сервер должен быть настроен с помощью политики EnterpriseInternalProxyServers. Эта коллекция может содержать не более 500 элементов.|
|enterpriseIPRanges|Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)|Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети. Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются. Безопасные место назначения для корпоративных данных открыть общий доступ в будут считаться местоположениях. Эта коллекция может содержать не более 500 элементов.|
|enterpriseInternalProxyServers|Коллекция String|Это список внутренних прокси-серверов, разделенных запятыми (например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"). Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете. Они считаются корпоративными серверами. Прокси-серверов только выполнять во время настройки EnterpriseCloudResources политики для принудительного трафика совпавших облачных ресурсов через эти прокси-серверы.|
|enterpriseIPRangesAreAuthoritative|Логический|Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей. Значение по умолчанию — false.|
|enterpriseProxyServers|Коллекция String|Это список прокси-серверов. Любой сервер не в этом списке считается вне предприятия.|
|enterpriseProxyServersAreAuthoritative|Логический|Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы. Значение по умолчанию: false.|
|neutralDomainResources|Коллекция String|Список имен доменов, которые можно использовать для рабочих или личных ресурса.|

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





