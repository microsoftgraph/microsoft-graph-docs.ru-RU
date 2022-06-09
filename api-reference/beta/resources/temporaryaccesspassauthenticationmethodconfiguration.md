---
title: Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности временного прохода доступа.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 073e89cccf4f63760bcf7bcc79a28c4a0c6f7e58
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971212"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности временного прохода доступа. Политика методов проверки подлинности определяет параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта **temporaryaccesspassauthenticationmethodconfiguration** .|
|[Обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration** .|
|[Удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Нет|Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** в конфигурацию по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|minimumLifetimeInMinutes|Целое|Минимальное время существования в минутах для любого временного приложенияAccessPass, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальное время существования в минутах для любого временного приложенияAccessPass, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|defaultLifetimeInMinutes|int|Время существования по умолчанию (в минутах) для временного приложенияAccessPass. Значение может быть в диапазоне от minimumLifetimeInMinutes до maximumLifetimeInMinutes.|
|defaultLength|int|Длина по умолчанию (в символах) временного объектаAccessPass от 8 до 48 символов.|
|isUsableOnce|Boolean   |Если `true`все проходы в клиенте будут ограничены однонастройным использованием. Если `false`, то можно создать клиент для однократного или многократного использования.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[Коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
}
```
