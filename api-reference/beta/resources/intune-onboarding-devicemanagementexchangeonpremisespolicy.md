---
title: Тип ресурса Девицеманажементексчанжеонпремисесполици
description: ОдноЭлементный объект, представляющий политику локальной политики Exchange, настроенную для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8605a3062d8808ea6a4d0b5397283f0ca82d920
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566572"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a>Тип ресурса Девицеманажементексчанжеонпремисесполици

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ОдноЭлементный объект, представляющий политику локальной политики Exchange, настроенную для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементексчанжеонпремисесполици](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[Девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Чтение свойств и связей объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .|
|[Обновление Девицеманажементексчанжеонпремисесполици](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[Девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Обновление свойств объекта [девицеманажементексчанжеонпремисесполици](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|Нотификатионконтент|Двоичный|Текст уведомления, который будет отправляться пользователям, помещенным в карантин этой политикой. Это HTML-кодированный массив байтов в кодировке UTF8.|
|Дефаултакцесслевел|[Девицеманажементексчанжеакцесслевел](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Состояние доступа по умолчанию в Exchange. Это правило применяется глобально ко всей организации Exchange. Возможные значения: `none`, `allow`, `block`, `quarantine`.|
|Акцессрулес|Коллекция [девицеманажементексчанжеакцессруле](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)|Список правил доступа к устройствам в Exchange. Правила доступа применяются глобально ко всей организации Exchange|
|Кновндевицеклассес|Коллекция [девицеманажементексчанжедевицекласс](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|Список классов устройств, известных для Exchange|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Параметры локального условного доступа в Exchange. Для локального условного доступа устройства должны быть зарегистрированы для доступа к почте и поддерживать его.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```





