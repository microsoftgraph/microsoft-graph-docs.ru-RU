---
title: тип ресурса iosVppAppAssignedLicense
description: Назначение лицензии программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a40d788a632ab9d746dba774388e9ab9df4323d9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820550"
---
# <a name="iosvppappassignedlicense-resource-type"></a>тип ресурса iosVppAppAssignedLicense

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии программы покупки тома iOS. Этот класс не поддерживает операции создания, удаления и обновления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[коллекция iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Список свойств и связей объектов [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Get iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Чтение свойств и связей объекта [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Создание iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Создайте новый [объект iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Удаление iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|Нет|Удаляет [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Обновление iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Обновление свойств объекта [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userEmailAddress|String|Адрес электронной почты пользователя.|
|userId|String|Идентификатор пользователя.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

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



