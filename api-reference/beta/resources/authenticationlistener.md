---
title: Тип ресурса authenticationListener
description: Определяет прослушиватель для оценки во время события проверки подлинности.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d89d7660fc2580b8fad185633b6b819df1a41aaf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720353"
---
# <a name="authenticationlistener-resource-type"></a>Тип ресурса authenticationListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет прослушиватель, который будет оцениваться при событии проверки подлинности при проверке подлинности. AuthenticationListener абстрактный и является базовым классом различных типов прослушивателей, которые можно оценить во время события проверки подлинности. 

Вы можете создать [invokeUserFlowListener](../resources/invokeuserflowlistener.md) для события onSignUpStart.. Это связывает приложение с пользовательским потоком, что позволяет самообслуживить [процесс регистрации.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) После того как приложение будет связано с потоком пользователей, пользователи, которые будут перейти к этому приложению, смогут инициировать процесс регистрации, который подавит гостевую учетную запись.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список onSignUpStart](../api/authenticationeventspolicy-list-onsignupstart.md)|[Коллекция authenticationListener](../resources/authenticationlistener.md)|Получите коллекцию ресурсов authenticationListener, поддерживаемых событием onSignupStart.|
|[Создание authenticationListener](../api/authenticationeventspolicy-post-onsignupstart.md)|[authenticationListener](../resources/authenticationlistener.md)|Создайте новый объект authenticationListener для события onSignupStart.|
|[Обновление authenticationListener](../api/authenticationlistener-update.md)|[authenticationListener](../resources/authenticationlistener.md)|Обновите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.|
|[Put authenticationListener](../api/authenticationlistener-put.md)|[authenticationListener](../resources/authenticationlistener.md)|Замените свойства объекта authenticationListener.|
|[Get authenticationListener](../api/authenticationlistener-get.md)|[authenticationListener](../resources/authenticationlistener.md)|Получите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.|
|[Удаление authenticationListener](../api/authenticationlistener-delete.md)|Нет|Удалите указанный прослушиватель, определенный для события onSignupStart в конвейере проверки подлинности.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор действия.|
|priority|Int32|Приоритет прослушиватель. Определяет порядок оценки, если событие имеет несколько прослушивателей. Приоритет оценивается от низкого до высокого.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель. В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
