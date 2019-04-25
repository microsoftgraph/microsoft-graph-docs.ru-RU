---
title: Тип ресурса Иосвппаппассигнедусерлиценсе
description: Назначение лицензии пользователя "программа приобретения объема" для iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87eec557f0844307988743578c795c38ae11289e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552165"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>Тип ресурса Иосвппаппассигнедусерлиценсе

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии пользователя "программа приобретения объема" для iOS. Этот класс не поддерживает операции создания, удаления и обновления.


НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосвппаппассигнедусерлиценсес](../api/intune-apps-iosvppappassigneduserlicense-list.md)|Коллекция [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md)|Список свойств и связей объектов [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Получение Иосвппаппассигнедусерлиценсе](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Чтение свойств и связей объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Создание Иосвппаппассигнедусерлиценсе](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Удаление Иосвппаппассигнедусерлиценсе](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Нет|Удаляет объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[Обновление Иосвппаппассигнедусерлиценсе](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Обновление свойств объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|Усеремаиладдресс|String|Адрес электронной почты пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|Имя участника-пользователя. НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





