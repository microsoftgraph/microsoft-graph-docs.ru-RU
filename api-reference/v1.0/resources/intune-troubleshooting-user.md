---
title: Тип ресурса user
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18955869ac60de15d797ebc79cf7e179673d310d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078786"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune-troubleshooting-user-list.md)|Коллекция объектов [user](../resources/intune-troubleshooting-user.md)|Список свойств и связей объектов [user](../resources/intune-troubleshooting-user.md).|
|[Получение пользователя](../api/intune-troubleshooting-user-get.md)|[user](../resources/intune-troubleshooting-user.md)|Чтение свойств и связей объекта [user](../resources/intune-troubleshooting-user.md).|
|[Создание пользователя](../api/intune-troubleshooting-user-create.md)|[user](../resources/intune-troubleshooting-user.md)|Создание объекта [user](../resources/intune-troubleshooting-user.md).|
|[Удаление пользователя](../api/intune-troubleshooting-user-delete.md)|Нет|Удаляет объект [user](../resources/intune-troubleshooting-user.md).|
|[Обновление пользователя](../api/intune-troubleshooting-user-update.md)|[user](../resources/intune-troubleshooting-user.md)|Обновление свойств объекта [user](../resources/intune-troubleshooting-user.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для пользователя.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для этого пользователя.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




