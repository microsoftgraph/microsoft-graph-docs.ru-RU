---
title: Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности временного прохода доступа, которая определяет параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: fbcaa5a1d941a29a12a54699021a7e6ee1b25c41
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094076"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности временного прохода доступа, которая определяет параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности [временного прохода доступа](temporaryaccesspassauthenticationmethod.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Чтение свойств и связей **временного объектаAccessPassAuthenticationMethodConfiguration** .|
|[Обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|Нет|Обновление свойств объекта **temporaryAccessPassAuthenticationMethodConfiguration** .|
|[Удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Нет|Возвращает объект **temporaryAccessPassAuthenticationMethodConfiguration** в конфигурацию по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultLength|Целое|Длина по умолчанию в символах объекта временного access Pass. Должен содержать от 8 до 48 символов.|
|defaultLifetimeInMinutes|Целое|Время существования по умолчанию в минутах для временного прохода доступа. Значение может быть любым целым числом между **minimumLifetimeInMinutes** и **maximumLifetimeInMinutes**.|
|id|String|Идентификатор политики метода проверки подлинности. Наследуется от [сущности](entity.md).|
|isUsableOnce|Boolean   |Если `true`все проходы в клиенте будут ограничены однонастройным использованием. Если `false`этот параметр передается клиенту, его можно создать для одноразового использования или повторного использования.|
|minimumLifetimeInMinutes|Целое|Минимальное время существования в минутах для любого временного прохода доступа, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальное время существования в минутах для любого временного прохода доступа, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|state|authenticationMethodState|Включен ли в клиенте метод временного сквозного доступа. Возможные значения: `enabled`, `disabled`. Наследуется [от authenticationMethodConfiguration](authenticationmethodconfiguration.md). |

## <a name="relationships"></a>Связи
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
  "isUsableOnce": "Boolean",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
