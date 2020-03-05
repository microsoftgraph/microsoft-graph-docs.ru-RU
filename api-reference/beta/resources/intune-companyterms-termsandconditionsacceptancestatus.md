---
title: Тип ресурса termsAndConditionsAcceptanceStatus
description: Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 232f7277479d1e6fa558deb0b365ca90d9522675
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487783"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a>Тип ресурса termsAndConditionsAcceptanceStatus

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект termsAndConditionsAcceptanceStatus представляет состояние принятия определенной политики условий для заданного пользователя. Чтобы получить доступ к корпоративному порталу, пользователям нужно принять последнюю версию условий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список termsAndConditionsAcceptanceStatuses](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|Коллекция [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Получение объекта termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);|Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Создание объекта termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md);|Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Удаление объекта termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|Нет|Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|
|[Обновление объекта termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта.|
|userDisplayName|String|Отображает имя пользователя, чье принятие представлено объектом.|
|acceptedVersion|Int32|Номер последней версии условий, принятых пользователем.|
|acceptedDateTime|DateTimeOffset|Дата и время последнего принятия условий пользователем.|
|userPrincipalName|String|UserPrincipalName пользователя, который принял термин.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Ссылка для перехода к назначенным условиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



