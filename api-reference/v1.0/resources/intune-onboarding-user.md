---
title: Тип ресурса user
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6056076d9e1d27ca6f8641c583e77feb9604c91b
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454772"
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



