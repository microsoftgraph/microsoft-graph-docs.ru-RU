---
title: Тип ресурса Мобилеаппполицисетитем
description: Класс, содержащий свойства, используемые для мобильного приложения Полицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 940371cb4bb2fe734924bc9e16669ab26b2f7a9f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201258"
---
# <a name="mobileapppolicysetitem-resource-type"></a>Тип ресурса Мобилеаппполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для мобильного приложения Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеаппполицисетитемс](../api/intune-policyset-mobileapppolicysetitem-list.md)|Коллекция [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md)|Список свойств и связей объектов [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Получение Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-get.md)|[мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md)|Чтение свойств и связей объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Создание Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-create.md)|[мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md)|Создание нового объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|
|[Удаление Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-delete.md)|Нет|Удаляет объект [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md).|
|[Обновление Мобилеаппполицисетитем](../api/intune-policyset-mobileapppolicysetitem-update.md)|[мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md)|Обновление свойств объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String.|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String.|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[полицисетстатус](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[Коде](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Установка цели Мобилеаппполицисетитем. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|settings|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|Параметры Мобилеаппполицисетитем.|

## <a name="relationships"></a>Отношения
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



