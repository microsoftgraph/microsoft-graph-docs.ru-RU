---
title: Тип ресурса Макосвппаппассигнедлиценсе
description: Назначение лицензии на MacOS Volume Purchase Program. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: adec4b71d1ec221f0f6ebb9b3c3792f160b452f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458830"
---
# <a name="macosvppappassignedlicense-resource-type"></a>Тип ресурса Макосвппаппассигнедлиценсе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии на MacOS Volume Purchase Program. Этот класс не поддерживает операции создания, удаления и обновления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосвппаппассигнедлиценсес](../api/intune-apps-macosvppappassignedlicense-list.md)|Коллекция [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Список свойств и связей объектов [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Получение Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-get.md)|[макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Чтение свойств и связей объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Создание Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-create.md)|[макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Создание нового объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|
|[Удаление Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-delete.md)|Нет|Удаляет объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Обновление Макосвппаппассигнедлиценсе](../api/intune-apps-macosvppappassignedlicense-update.md)|[макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md)|Обновление свойств объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|усеремаиладдресс|String|Адрес электронной почты пользователя.|
|userId|String|Идентификатор пользователя.|
|userName|String|Имя пользователя.|
|userPrincipalName|Строка|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
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



