---
title: тип ресурса dataSharingConsent
description: Сведения о согласии на обмен данными.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06d712ffa94b4308c7234b45ffba5d0ab6c05423
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791132"
---
# <a name="datasharingconsent-resource-type"></a>тип ресурса dataSharingConsent

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о согласии на обмен данными.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[коллекция dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Список свойств и связей объектов [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Get dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Чтение свойств и связей объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Создание dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Создание нового [объекта dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Удаление dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Нет|Удаляет [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Обновление dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Обновление свойств объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Действие consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID согласия для общего доступа к данным|
|serviceDisplayName|Строка|Имя отображения потока работы службы|
|termsUrl|Строка|TermsUrl для согласия на обмен данными|
|granted|Логический|Предоставлено состояние для согласия на обмен данными|
|grantDateTime|DateTimeOffset|Для этой учетной записи было предоставлено согласие на время|
|grantedByUpn|String|Upn пользователя, который предоставил согласие для этой учетной записи|
|grantedByUserId|Строка|UserId пользователя, который предоставил согласие для этой учетной записи|

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



