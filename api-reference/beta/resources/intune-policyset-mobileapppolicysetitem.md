---
title: Тип ресурса Мобилеаппполицисетитем
description: Класс, содержащий свойства, используемые для мобильного приложения Полицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5d821063615d06e436bbbd2620eed71880757d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527608"
---
# <a name="mobileapppolicysetitem-resource-type"></a>Тип ресурса Мобилеаппполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для мобильного приложения Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеаппполицисетитемс](../api/intune-policyset-mobileapppolicysetitem-list.md)|Коллекция [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md)|Список свойств и связей объектов [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Получение Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-get.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Чтение свойств и связей объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Создание Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-create.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Создание нового объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Удаление Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-delete.md)|Нет|Удаляет объект [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md).|
|[Обновление Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-update.md)|[mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md)|Обновление свойств объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|Строка|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|Строка|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция String|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Установка цели Мобилеаппполицисетитем. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|settings|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|Параметры Мобилеаппполицисетитем.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "intent": "String",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



