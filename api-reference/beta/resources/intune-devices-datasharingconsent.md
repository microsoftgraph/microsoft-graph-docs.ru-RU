---
title: Тип ресурса Даташарингконсент
description: Сведения о согласии общего доступа к данным.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f98c2967eb9d3e14b0f8e219547aa73104d67614
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785037"
---
# <a name="datasharingconsent-resource-type"></a>Тип ресурса Даташарингконсент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|сервицедисплайнаме|String|Отображаемое имя рабочего процесса службы|
|термсурл|String|Термсурл для согласия общего доступа к данным|
|granted|Логический|Состояние предоставления согласия на общий доступ к данным|
|грантдатетиме|DateTimeOffset|Для этой учетной записи предоставлено согласие по времени|
|грантедбюпн|String|Имя участника-пользователя, которому назначено согласие для этой учетной записи.|
|грантедбюсерид|String|UserId пользователя, который предоставил согласие для этой учетной записи|

## <a name="relationships"></a>Связи
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



