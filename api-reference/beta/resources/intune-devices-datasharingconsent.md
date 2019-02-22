---
title: Тип ресурса Даташарингконсент
description: Сведения о согласии общего доступа к данным.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ef8b899c6fa7645b31cd77ada7420b0f753a60
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174652"
---
# <a name="datasharingconsent-resource-type"></a>Тип ресурса Даташарингконсент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о согласии общего доступа к данным.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Даташарингконсентс](../api/intune-devices-datasharingconsent-list.md)|Коллекция [даташарингконсент](../resources/intune-devices-datasharingconsent.md)|Список свойств и связей объектов [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .|
|[Получение Даташарингконсент](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Чтение свойств и связей объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .|
|[Создание Даташарингконсент](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Создание нового объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .|
|[Удаление Даташарингконсент](../api/intune-devices-datasharingconsent-delete.md)|Нет|Удаляет объект [даташарингконсент](../resources/intune-devices-datasharingconsent.md).|
|[Обновление Даташарингконсент](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Обновление свойств объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .|
|[Действие consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор согласия общего доступа к данным|
|Сервицедисплайнаме|String|Отображаемое имя рабочего процесса службы|
|Термсурл|String|Термсурл для согласия общего доступа к данным|
|granted|Логический|Состояние предоставления согласия на общий доступ к данным|
|Грантдатетиме|DateTimeOffset|Для этой учетной записи предоставлено согласие по времени|
|Грантедбюпн|String|Имя участника-пользователя, которому назначено согласие для этой учетной записи.|
|Грантедбюсерид|String|UserId пользователя, который предоставил согласие для этой учетной записи|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```




