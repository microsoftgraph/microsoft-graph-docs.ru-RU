---
title: Тип ресурса Мдмвиндовсинформатионпротектионполициполицисетитем
description: Класс, содержащий свойства, используемые для политики Windows Information Protection для MDM Полицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fb67456954652c6f468cd163815ebeb198e2dc3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288077"
---
# <a name="mdmwindowsinformationprotectionpolicypolicysetitem-resource-type"></a>Тип ресурса Мдмвиндовсинформатионпротектионполициполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для политики Windows Information Protection для MDM Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мдмвиндовсинформатионпротектионполициполицисетитемс](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-list.md)|Коллекция [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Список свойств и связей объектов [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .|
|[Получение Мдмвиндовсинформатионпротектионполициполицисетитем](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-get.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Чтение свойств и связей объекта [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .|
|[Создание Мдмвиндовсинформатионпротектионполициполицисетитем](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-create.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Создание нового объекта [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .|
|[Удаление Мдмвиндовсинформатионпротектионполициполицисетитем](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-delete.md)|Нет|Удаляет объект [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).|
|[Обновление Мдмвиндовсинформатионпротектионполициполицисетитем](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-update.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Обновление свойств объекта [мдмвиндовсинформатионпротектионполициполицисетитем](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|String|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
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
  ]
}
```




