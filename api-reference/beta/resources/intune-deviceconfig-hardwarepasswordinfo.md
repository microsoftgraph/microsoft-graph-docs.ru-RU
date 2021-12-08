---
title: тип ресурса hardwarePasswordInfo
description: Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fd663fbcfd721e6fd6ed762d0de2b107503ec2c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345618"
---
# <a name="hardwarepasswordinfo-resource-type"></a>тип ресурса hardwarePasswordInfo

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность настраивать параметры оборудования и биосов на зарегистрированных устройствах windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список hardwarePasswordInfos](../api/intune-deviceconfig-hardwarepasswordinfo-list.md)|[коллекция hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Список свойств и связей объектов [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Get hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-get.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Чтение свойств и связей объекта [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Создание hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-create.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Создание нового [объекта hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Удаление hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-delete.md)|Нет|Удаляет [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md).|
|[Обновление hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-update.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Обновление свойств объекта [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для информации о аппаратном пароле|
|serialNumber|String|Серийный номер устройства|
|currentPassword|Строка|Текущий пароль устройства|
|previousPasswords|Коллекция String|Список предыдущих паролей устройств|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwarePasswordInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "id": "String (identifier)",
  "serialNumber": "String",
  "currentPassword": "String",
  "previousPasswords": [
    "String"
  ]
}
```




