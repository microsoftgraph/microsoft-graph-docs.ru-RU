---
title: Тип ресурса Макосвппаппассигнедлиценсе
description: Назначение лицензии на MacOS Volume Purchase Program. Этот класс не поддерживает операции создания, удаления и обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67031c6bdd81052dbc41264104bc5a02566cfd51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012557"
---
# <a name="macosvppappassignedlicense-resource-type"></a>Тип ресурса Макосвппаппассигнедлиценсе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии на MacOS Volume Purchase Program. Этот класс не поддерживает операции создания, удаления и обновления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосвппаппассигнедлиценсес](../api/intune-apps-macosvppappassignedlicense-list.md)|Коллекция [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Список свойств и связей объектов [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Получение Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-get.md)|[Макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Чтение свойств и связей объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Создание Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-create.md)|[Макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Создание нового объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Удаление Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-delete.md)|Нет|Удаляет объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Обновление Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-update.md)|[Макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Обновление свойств объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|Усеремаиладдресс|String|Адрес электронной почты пользователя.|
|userId|String|Идентификатор пользователя.|
|userName|String|Имя пользователя.|
|userPrincipalName|Строка|Имя участника-пользователя.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





