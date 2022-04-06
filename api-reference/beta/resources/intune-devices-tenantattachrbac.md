---
title: тип ресурса tenantAttachRBAC
description: Объект Singleton, который выступает в качестве контейнера для функциональность присоединений клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af582f15444821fba9e36cf23ef1f2c4075ad57c
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631423"
---
# <a name="tenantattachrbac-resource-type"></a>тип ресурса tenantAttachRBAC

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Singleton, который выступает в качестве контейнера для функциональность присоединений клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получить tenantAttachRBAC](../api/intune-devices-tenantattachrbac-get.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|Чтение свойств и отношений объекта [tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) .|
|[Обновление tenantAttachRBAC](../api/intune-devices-tenantattachrbac-update.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|Обновление свойств объекта [tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) .|
|[включить действие](../api/intune-devices-tenantattachrbac-enable.md)|Нет|Н/Д|
|[функция getState](../api/intune-devices-tenantattachrbac-getstate.md)|[tenantAttachRBACState](../resources/intune-devices-tenantattachrbacstate.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAttachRBAC"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantAttachRBAC",
  "id": "String (identifier)"
}
```




