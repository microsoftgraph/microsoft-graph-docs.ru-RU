---
title: тип ресурса macOsVppAppAssignedLicense
description: Назначение лицензии программы тома MacOS. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc32cd6b661b7f89453da1c6ddf3b3320686907fd14c3777d9ab663160b7eae6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173319"
---
# <a name="macosvppappassignedlicense-resource-type"></a>тип ресурса macOsVppAppAssignedLicense

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение лицензии программы тома MacOS. Этот класс не поддерживает операции создания, удаления и обновления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[коллекция macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Список свойств и связей объектов [macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Get macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Чтение свойств и связей объекта [macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Создание macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Создание нового [объекта macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Удаление macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|Нет|Удаляет [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Обновление macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Обновление свойств объекта [macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userEmailAddress|Строка|Адрес электронной почты пользователя.|
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




