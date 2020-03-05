---
title: Тип ресурса Манажедаллдевицецертификатестате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be36b8c62d661957158dce03514e3c20bc4c0c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526064"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>Тип ресурса Манажедаллдевицецертификатестате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажедаллдевицецертификатестатес](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|Коллекция [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Список свойств и связей объектов [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Получение Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Чтение свойств и связей объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Создание Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Удаление Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|Нет|Удаляет объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).|
|[Обновление Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|цертификатеревокестатус|[цертификатеревокатионстатус](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзыв состояния. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|манажеддевицедисплайнаме|String|Отображаемое имя устройства|
|userPrincipalName|String|Имя субъекта-пользователя|
|цертификатикспиратиондатетиме|DateTimeOffset|Дата окончания срока действия сертификата|
|цертификатеиссуернаме|String|Издатель|
|certificateThumbprint|String|Отпечаток|
|цертификатесериалнумбер|String|Серийный номер|
|цертификатесубжектнаме|String|Имя субъекта сертификата|
|цертификатекэйусажес|Int32|Использование ключа|
|цертификатикстендедкэйусажес|String|Расширенное использование ключа|
|цертификатеиссуанцедатетиме|DateTimeOffset|Дата выпуска|

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



