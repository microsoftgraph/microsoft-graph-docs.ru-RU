---
title: Тип ресурса iosVppAppAssignedLicense
description: операций ввода-вывода программы покупки корпоративного лицензионного назначения. Этот класс не поддерживает операции создания, удаления и обновления.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5d2588cd8ceeae44b7e4150544a984c68d4d90e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991216"
---
# <a name="iosvppappassignedlicense-resource-type"></a>Тип ресурса iosVppAppAssignedLicense

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

операций ввода-вывода программы покупки корпоративного лицензионного назначения. Этот класс не поддерживает операции создания, удаления и обновления.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) коллекции|Свойства списка и связей объектов [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Получение iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Чтение свойства и связи объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Создание iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Создание нового объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|
|[Удаление iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|Нет|Удаляет [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Обновление iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Обновление свойства объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .|

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





