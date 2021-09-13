---
title: тип ресурса dataSharingConsent
description: Сведения о согласии на обмен данными.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92c012f994c3e5aa3630f05632d48df764a432d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057329"
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
|[Get dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Чтение свойств и связей объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Создание dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Создание нового [объекта dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Удаление dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Нет|Удаляет [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Обновление dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Обновление свойств объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)|
|[Действие consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID согласия для общего доступа к данным|
|serviceDisplayName|String|Имя отображения потока работы службы|
|termsUrl|String|TermsUrl для согласия на обмен данными|
|granted|Логическое|Предоставлено состояние для согласия на обмен данными|
|grantDateTime|DateTimeOffset|Для этой учетной записи было предоставлено согласие на время|
|grantedByUpn|String|Upn пользователя, который предоставил согласие для этой учетной записи|
|grantedByUserId|String|UserId пользователя, который предоставил согласие для этой учетной записи|

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



