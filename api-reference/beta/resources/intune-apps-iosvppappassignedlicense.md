---
title: Тип ресурса Иосвппаппассигнедлиценсе
description: Назначение лицензии на программу приобретения тома для iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc967be6bc808ea6443f2fd6333b6313b11ab596
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950377"
---
# <a name="iosvppappassignedlicense-resource-type"></a>Тип ресурса Иосвппаппассигнедлиценсе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии на программу приобретения тома для iOS. Этот класс не поддерживает операции создания, удаления и обновления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосвппаппассигнедлиценсес](../api/intune-apps-iosvppappassignedlicense-list.md)|Коллекция [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|Список свойств и связей объектов [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Получение Иосвппаппассигнедлиценсе](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Чтение свойств и связей объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Создание Иосвппаппассигнедлиценсе](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Создание нового объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Удаление Иосвппаппассигнедлиценсе](../api/intune-apps-iosvppappassignedlicense-delete.md)|Нет|Удаляет объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Обновление Иосвппаппассигнедлиценсе](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Обновление свойств объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|Усеремаиладдресс|Строка|Адрес электронной почты пользователя.|
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
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```




