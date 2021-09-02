---
title: тип ресурса iosVppAppAssignedUserLicense
description: Назначение лицензии пользователя программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a933d23410a828609bbb8e14466bd112657afda6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802812"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>тип ресурса iosVppAppAssignedUserLicense

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии пользователя программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.


Наследует [от iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[коллекция iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Список свойств и связей объектов [iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Get iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Чтение свойств и связей объекта [iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Создание iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Создайте новый [объект iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Удаление iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Нет|Удаляет [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[Обновление iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Обновление свойств объекта [iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|Строка|Адрес электронной почты пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|Идентификатор пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|Имя пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|Имя участника-пользователя. Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>Связи
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



