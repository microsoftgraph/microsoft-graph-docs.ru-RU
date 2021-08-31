---
title: Тип ресурса pfxRecryptionRequest
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a84f5514e13633c1c5a2ed5f6ffc5ce5b9130eea
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805291"
---
# <a name="pfxrecryptionrequest-resource-type"></a>Тип ресурса pfxRecryptionRequest

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список pfxRecryptionRequests](../api/intune-raimportcerts-pfxrecryptionrequest-list.md)|[Коллекция pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Список свойств и связей объектов [pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Get pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-get.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Чтение свойств и связей объекта [pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Создание pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-create.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Создайте новый [объект pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|
|[Удаление pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-delete.md)|Нет|Удаляет [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md).|
|[Обновление pfxRecryptionRequest](../api/intune-raimportcerts-pfxrecryptionrequest-update.md)|[pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|Обновление свойств объекта [pfxRecryptionRequest.](../resources/intune-raimportcerts-pfxrecryptionrequest.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|profileId|Guid|Пока не задокументировано.|
|отпечатки пальцев|String|Пока не задокументировано.|
|deviceKeyThumbprint|String|Пока не задокументировано.|
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



