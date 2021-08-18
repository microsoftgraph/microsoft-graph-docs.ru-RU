---
title: тип ресурса microsoftTunnelSite
description: Сущность, представляюая Microsoft Tunnel сайт
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de026e42f21b29327620f3170fa4d3e8117af01342b0e494bafa949efb1c8261
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178866"
---
# <a name="microsofttunnelsite-resource-type"></a>тип ресурса microsoftTunnelSite

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая Microsoft Tunnel сайт

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[коллекция microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Список свойств и связей объектов [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Получите microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Чтение свойств и связей объекта [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Создание microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Создайте новый [объект microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Удаление microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Нет|Удаляет [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Обновление microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Обновление свойств объекта [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelSite|
|displayName|String|Имя отображения MicrosoftTunnelSite|
|description|Строка|Описание MicrosoftTunnelSite|
|publicAddress|Строка|Имя или IP-адрес общественного домена MicrosoftTunnelSite|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|MicrosoftTunnelConfiguration, примененная к этому MicrosoftTunnelSite|
|microsoftTunnelServers|[коллекция microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Список microsoftTunnelServers, зарегистрированных в этом MicrosoftTunnelSite|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




