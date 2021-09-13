---
title: тип ресурса managedAllDeviceCertificateState
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84ef0315f30bb249a393b3994524ea87acca5bab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075482"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>тип ресурса managedAllDeviceCertificateState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedAllDeviceCertificateStates](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|[коллекция managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Список свойств и связей [объектов managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[УправлениеAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Чтение свойств и связей [объекта managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[Создание managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Создайте новый [объект managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|
|[Удаление managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|Нет|Удаляет [управляемыйAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).|
|[Обновление managedAllDeviceCertificateState](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Обновление свойств объекта [managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзови статус. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateRevokeStatusLastChangeDateTime|DateTimeOffset|Время последнего изменения состояния отвода|
|managedDeviceDisplayName|String|Имя отображения устройства|
|userPrincipalName|String|Имя субъекта-пользователя|
|certificateExpirationDateTime|DateTimeOffset|Дата истечения срока действия сертификата|
|certificateIssuerName|String|Издатель|
|certificateThumbprint|String|Thumbprint|
|certificateSerialNumber|String|Серийный номер|
|certificateSubjectName|String|Имя субъекта сертификата|
|certificateKeyUsages|Int32|Использование ключей|
|certificateExtendedKeyUsages|String|Расширенное использование ключей|
|certificateIssuanceDateTime|DateTimeOffset|Дата выпуска|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "certificateRevokeStatusLastChangeDateTime": "String (timestamp)",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```



