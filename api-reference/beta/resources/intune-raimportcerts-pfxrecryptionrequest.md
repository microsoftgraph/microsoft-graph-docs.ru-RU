---
title: Тип ресурса pfxRecryptionRequest
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 904ce75ba1b3afb135ba2788dcde4c629c34a2ff
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868815"
---
# <a name="pfxrecryptionrequest-resource-type"></a>Тип ресурса pfxRecryptionRequest

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

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




