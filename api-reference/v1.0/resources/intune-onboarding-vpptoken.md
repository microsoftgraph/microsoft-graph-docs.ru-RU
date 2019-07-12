---
title: Тип ресурса vppToken
description: Вы приобрели несколько лицензий для приложений для iOS по программе корпоративных покупок Apple Volume Purchase Program для бизнеса или образовательных учреждений. Это включает настройку учетной записи Apple VPP с веб-сайта Apple и передачу токена Apple VPP для бизнеса или образовательных учреждений в Intune. Затем вы можете синхронизировать данные корпоративных покупок с помощью Intune и отслеживать использование приложения, приобретенного по программе корпоративных покупок. Вы можете передать несколько токенов Apple VPP для бизнеса или образовательных учреждений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d12071be045eb9c0e7b057af517941ee14d7aea2
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621314"
---
# <a name="vpptoken-resource-type"></a>Тип ресурса vppToken

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы приобрели несколько лицензий для приложений для iOS по программе корпоративных покупок Apple Volume Purchase Program для бизнеса или образовательных учреждений. Это включает настройку учетной записи Apple VPP с веб-сайта Apple и передачу токена Apple VPP для бизнеса или образовательных учреждений в Intune. Затем вы можете синхронизировать данные корпоративных покупок с помощью Intune и отслеживать использование приложения, приобретенного по программе корпоративных покупок. Вы можете передать несколько токенов Apple VPP для бизнеса или образовательных учреждений.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список VPP токенов](../api/intune-onboarding-vpptoken-list.md)|Коллекция [VPP токенов](../resources/intune-onboarding-vpptoken.md)|Список свойств и связей объектов [VPP токен](../resources/intune-onboarding-vpptoken.md).|
|[Получить VPP токен](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Чтение свойств и связей объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).|
|[Создать VPP токен](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Создайте новый объект [VPP токен](../resources/intune-onboarding-vpptoken.md).|
|[Удалить VPP токен](../api/intune-onboarding-vpptoken-delete.md)|Отсутствует|Удаляет [VPP токен](../resources/intune-onboarding-vpptoken.md).|
|[Обновить VPP токен](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).|
|[Действие syncLicenses](../api/intune-onboarding-vpptoken-synclicenses.md)|[VPP токен](../resources/intune-onboarding-vpptoken.md)|Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Создается автоматически при создании appleVolumePurchaseProgramToken. Это ключ объекта.|
|organizationName|String|Организация, связанная с токеном Apple Volume Purchase Program.|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.|
|appleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|Дата и время завершения срока действия токена Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|Время последнего выполнения синхронизации приложения со службой Apple Volume Purchase Program с помощью маркера Apple Volume Purchase Program.|
|токен|String|Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.|
|состояние|[Впптокенстате](../resources/intune-onboarding-vpptokenstate.md)|Текущее состояние токена Apple Volume Purchase Program. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[Впптокенсинкстатус](../resources/intune-onboarding-vpptokensyncstatus.md)|Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program. Возможные значения: `none`, `inProgress`, `completed`, `failed`. Возможные значения: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Логическое|Автоматически обновятся все приложения, не только для токена VPP.|
|countryOrRegion|Строка|Автоматически обновятся все приложения, не только для токена VPP.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```



