---
title: тип ресурса mobilityManagementPolicy
description: Политика управления мобильностью представляет политику автоматической регистрации для приложения управления мобильностью, настроенного в Azure AD.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6c2035d96293a28f4d8289606df709fc64d9c3e7
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401545"
---
# <a name="mobilitymanagementpolicy-resource-type"></a>тип ресурса mobilityManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В Azure AD политика управления мобильностью представляет конфигурацию автоматической регистрации для приложения управления мобильностью (MDM или MAM). Эти политики применимы только к устройствам на основе Windows 10 оси и ее производных (Surface Hub, Hololens и т.д.). [Автоматическая регистрация позволяет](/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal) организациям автоматически регистрировать устройства в выбранное приложение управления мобильностью в рамках процесса регистрации [Azure AD](/azure/active-directory/devices/concept-azure-ad-join) или [Azure AD](/azure/active-directory/devices/concept-azure-ad-register) на Windows 10 устройствах.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список mobileDeviceManagementPolicies](../api/mobiledevicemanagementpolicies-list.md)|[коллекция mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Получите список объектов [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) и их свойств для приложений для управления мобильными устройствами.|
|[Get mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными устройствами.|
|[Обновление mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-update.md)|Нет|Обновление свойств объекта [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными устройствами.|
|[В список вошли Группы mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-list-includedgroups.md)|Коллекция [group](../resources/group.md)|В список включены группы для [объекта mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными устройствами.|
|[Добавление группы в mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-post-includedgroups.md)|Нет|Добавьте группу в [объект mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными устройствами.|
|[Удаление группы из mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-delete-includedgroups.md)|Нет|Удаление группы из объекта [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными устройствами.|
|[Список mobileAppManagementPolicies](../api/mobileappmanagementpolicies-list.md)|[коллекция mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Получите список объектов [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) и их свойств для приложений для управления мобильными приложениями.|
|[Get mobileAppManagementPolicy](../api/mobileappmanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными приложениями.|
|[Обновление mobileAppManagementPolicy](../api/mobileappmanagementpolicies-update.md)|Нет|Обновление свойств объекта [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными приложениями.|
|[В список вошли Группы mobileAppManagementPolicy](../api/mobileappmanagementpolicies-list-includedgroups.md)|Коллекция [group](../resources/group.md)|В список вошли группы для [объекта mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными приложениями.|
|[Добавление группы в mobileAppManagementPolicy](../api/mobileappmanagementpolicies-post-includedgroups.md)|Нет|Добавьте группу в [объект mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными приложениями.
|[Удаление группы из mobileAppManagementPolicy](../api/mobileappmanagementpolicies-delete-includedgroups.md)|Нет|Удаление группы из [объекта mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) для приложения для управления мобильными приложениями.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|appliesTo|policyScope|Указывает область действия пользователя политики управления мобильностью. Возможные значения: `none`, `all`, `selected`.|
|complianceUrl|String|URL-адрес соответствия приложению управления мобильностью.|
|description|String|Описание приложения для управления мобильностью.|
|discoveryUrl|String|Обнаружение URL-адреса приложения для управления мобильностью.|
|displayName|String|Отображение имени приложения управления мобильностью.|
|id|String|Объект Id приложения управления мобильностью.|
|isValid|Boolean|Допустима ли политика. Недействительные политики могут не обновляться и должны быть удалены.|
|termsOfUseUrl|String|Условия использования URL-адреса приложения для управления мобильностью.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|includedGroups|Коллекция [group](../resources/group.md)|Azure AD groups under the scope of the mobility management application if appliesTo is `selected`|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobilityManagementPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "isValid": "Boolean",
  "termsOfUseUrl": "String"
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "mobilityManagementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
