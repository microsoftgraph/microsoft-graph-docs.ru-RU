---
title: Тип ресурса windowsAssignedAccessProfile
description: Назначенный профиль доступа для Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 893e81e544286c6877b9443d96f610acb939e934
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972854"
---
# <a name="windowsassignedaccessprofile-resource-type"></a>Тип ресурса windowsAssignedAccessProfile

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Назначенный профиль доступа для Windows.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsAssignedAccessProfiles](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) коллекции|Свойства списка и связей объектов [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Получение windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Чтение свойства и связи объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Создание windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Создание нового объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|
|[Удаление windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|Нет|Удаляет [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).|
|[Обновление windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|Обновление свойства объекта [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|Имя_профиля|Строка|Это понятное имя, используемое для идентификации групп приложений, макет эти приложения в меню Пуск и пользователи, которым назначена эта конфигурация киоска.|
|showTaskBar|Логический|Этот параметр позволяет администратору задать, отображается ли панель задач.|
|appUserModelIds|Коллекция String|Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.|
|desktopAppPaths|Коллекция String|Ниже приведены пути в настольных приложений, которые будут доступны в меню Пуск и только приложения пользователь будет иметь возможность запуска.|
|userAccounts|Коллекция String|Учетные записи пользователей, которые будут заблокированы для этой базовой конфигурации.|
|startMenuLayoutXml|Binary|Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета. XML должен быть в двоичном формате.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





