---
title: Тип ресурса Пфксрекриптионрекуест
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 904ce75ba1b3afb135ba2788dcde4c629c34a2ff
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307167"
---
# <a name="pfxrecryptionrequest-resource-type"></a>Тип ресурса Пфксрекриптионрекуест

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Пфксрекриптионрекуестс](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|Коллекция [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Список свойств и связей объектов [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Получение Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Чтение свойств и связей объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Создание Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Создание нового объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Удаление Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|Нет|Удаляет объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md).|
|[Обновление Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Обновление свойств объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|профилеид|Guid|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|девицекэйсумбпринт|String|Пока не задокументировано.|
|status|Int32|Пока не задокументировано.|
|sourceType|Int32|Пока не задокументировано.|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|isDeleted|Boolean|Н/Д|
|eTag|String|Н/Д|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxRecryptionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "profileId": "Guid",
  "thumbprint": "String",
  "deviceKeyThumbprint": "String",
  "status": 1024,
  "sourceType": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "isDeleted": true,
  "eTag": "String"
}
```




