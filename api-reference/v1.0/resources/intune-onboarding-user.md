---
title: Тип ресурса user
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30c01a5217890a639137bbd1989f52d5f9090f86
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731206"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune-onboarding-user-list.md)|Коллекция объектов [user](../resources/intune-onboarding-user.md)|Список свойств и связей объектов [user](../resources/intune-onboarding-user.md).|
|[Получение пользователя](../api/intune-onboarding-user-get.md)|[user](../resources/intune-onboarding-user.md)|Чтение свойств и связей объекта [user](../resources/intune-onboarding-user.md).|
|[Создание пользователя](../api/intune-onboarding-user-create.md)|[user](../resources/intune-onboarding-user.md)|Создание объекта [user](../resources/intune-onboarding-user.md).|
|[Удаление пользователя](../api/intune-onboarding-user-delete.md)|Нет|Удаляет объект [user](../resources/intune-onboarding-user.md).|
|[Обновление пользователя](../api/intune-onboarding-user-update.md)|[user](../resources/intune-onboarding-user.md)|Обновление свойств объекта [user](../resources/intune-onboarding-user.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|

## <a name="relationships"></a>Связи
Нет

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
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```





