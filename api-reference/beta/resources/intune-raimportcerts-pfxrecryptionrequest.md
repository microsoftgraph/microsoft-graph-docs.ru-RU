---
title: Тип ресурса Пфксрекриптионрекуест
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 308b487ad77558ef5e847599e7b4a130c2ef6603
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741516"
---
# <a name="pfxrecryptionrequest-resource-type"></a>Тип ресурса Пфксрекриптионрекуест

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Пфксрекриптионрекуестс](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|Коллекция [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Список свойств и связей объектов [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Получение Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[Пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Чтение свойств и связей объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Создание Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[Пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Создание нового объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|
|[Удаление Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|Нет|Удаляет объект [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md).|
|[Обновление Пфксрекриптионрекуест](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[Пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Обновление свойств объекта [пфксрекриптионрекуест](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|Профилеид|GUID|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|Девицекэйсумбпринт|String|Пока не задокументировано.|
|status|Int32|Пока нет описания|
|sourceType|Int32|Пока нет описания|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|isDeleted|Boolean|Пока не задокументировано|
|eTag|String|Пока не задокументировано.|

## <a name="relationships"></a>Отношения
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





