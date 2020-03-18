---
title: Тип ресурса Манажедапппротектионполицисетитем
description: Класс, содержащий свойства, используемые для Полицисетитем защиты управляемых приложений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e8bdc277f92d30f6506b5528bc00816d8639e65
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775740"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a>Тип ресурса Манажедапппротектионполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для Полицисетитем защиты управляемых приложений.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажедапппротектионполицисетитемс](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|Коллекция [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Список свойств и связей объектов [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .|
|[Получение Манажедапппротектионполицисетитем](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Чтение свойств и связей объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .|
|[Создание Манажедапппротектионполицисетитем](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Создание нового объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .|
|[Удаление Манажедапппротектионполицисетитем](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|Нет|Удаляет объект [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md).|
|[Обновление Манажедапппротектионполицисетитем](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|Обновление свойств объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция String|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|таржетедаппманажементлевелс|String|Таржетедаппманажементлевелс Манажедаппполицисетитем.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtectionPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
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
  "targetedAppManagementLevels": "String"
}
```



