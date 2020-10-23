---
title: Тип ресурса Даташарингконсент
description: Сведения о согласии общего доступа к данным.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0235abf74d96e5ccff888253e977bd9951bbc3cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703652"
---
# <a name="datasharingconsent-resource-type"></a>Тип ресурса Даташарингконсент

Пространство имен: microsoft.graph

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
|id|Строка|Идентификатор согласия общего доступа к данным|
|сервицедисплайнаме|Строка|Отображаемое имя рабочего процесса службы|
|термсурл|Строка|Термсурл для согласия общего доступа к данным|
|granted|Логический|Состояние предоставления согласия на общий доступ к данным|
|грантдатетиме|DateTimeOffset|Для этой учетной записи предоставлено согласие по времени|
|грантедбюпн|Строка|Имя участника-пользователя, которому назначено согласие для этой учетной записи.|
|грантедбюсерид|Строка|UserId пользователя, который предоставил согласие для этой учетной записи|

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





