---
title: Тип ресурса microsoftTunnelServerLogCollectionResponse
description: Сущность, в которую хранится состояние коллекции журналов сервера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2162feeec570a0d19739036f902542f374f6d767
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162474"
---
# <a name="microsofttunnelserverlogcollectionresponse-resource-type"></a>Тип ресурса microsoftTunnelServerLogCollectionResponse

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, в которую хранится состояние коллекции журналов сервера.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelServerLogCollectionResponses](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-list.md)|[Коллекция microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Список свойств и связей объектов [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Get microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-get.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Чтение свойств и связей объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Создание microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-create.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Создание объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Удаление microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-delete.md)|Нет|Удаляет [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|
|[Обновление microsoftTunnelServerLogCollectionResponse](../api/intune-mstunnel-microsofttunnelserverlogcollectionresponse-update.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Обновление свойств объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный ИД сущности|
|status|[microsoftTunnelLogCollectionStatus](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|Состояние сбора журналов. Возможные значения: `pending`, `completed`, `failed`.|
|startDateTime|DateTimeOffset|Время начала сбора журналов |
|endDateTime|DateTimeOffset|Время окончания собранных журналов|
|sizeInBytes|Int64|Размер журналов в ветвях|

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




