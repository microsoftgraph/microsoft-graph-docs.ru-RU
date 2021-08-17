---
title: тип ресурса microsoftTunnelServerLogCollectionResponse
description: Объект, который хранит состояние коллекции журнала сервера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59542a568047fab6103a3af9520a2239ddceaad6ebe97161aefd7d8e49f0042d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178880"
---
# <a name="microsofttunnelserverlogcollectionresponse-resource-type"></a>тип ресурса microsoftTunnelServerLogCollectionResponse

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, который хранит состояние коллекции журнала сервера.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelServerLogCollectionResponses](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-list.md)|[коллекция microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Список свойств и связей [объектов microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Получите microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-get.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Чтение свойств и связей объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Создание microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-create.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Создайте [новый объект microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Удаление microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-delete.md)|Нет|Удаляет [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).|
|[Обновление microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-update.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Обновление свойств объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный ID объекта|
|status|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|Состояние коллекции журналов. Возможные значения: `pending`, `completed`, `failed`.|
|startDateTime|DateTimeOffset|Время начала собранных журналов |
|endDateTime|DateTimeOffset|Время окончания собранных журналов|
|sizeInBytes|Int64|Размер журналов в bytes|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServerLogCollectionResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "String (identifier)",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "sizeInBytes": 1024
}
```




