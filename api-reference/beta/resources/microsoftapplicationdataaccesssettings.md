---
title: тип ресурса microsoftApplicationDataAccessSettings
description: Представляет параметры для определения доступа из приложений Майкрософт Microsoft 365 данных, принадлежащих пользователям в организации. Например, при надлежащей авторизации доступ к Microsoft 365 приложениям (таким как Word и Excel) могут получать доступ к данным Microsoft 365 пользователей, а также к другим приложениям Майкрософт (например, Windows), а также к данным.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 049089e4c3246beed9f459831cd7903dea9e4ce3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589872"
---
# <a name="microsoftapplicationdataaccesssettings-resource-type"></a>тип ресурса microsoftApplicationDataAccessSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет _параметры_, которые указывают доступ из приложений Майкрософт к Microsoft 365 данным, принадлежащим пользователям в организации. Например, при надлежащей авторизации доступ к Microsoft 365 пользователям могут получать только Microsoft 365 приложения (например, Word и Excel), а также могут ли другие приложения Майкрософт (например, Windows) получать доступ к данным.

Примеры Microsoft 365 в организации включают документы Word, Excel и PowerPoint, Outlook сообщения и записи Teams собраний, к которым пользователь в приложении Майкрософт был должным образом уполномочен к доступу.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список microsoftApplicationDataAccessSettings](../api/organizationsettings-list-microsoftapplicationdataaccess.md)|[MicrosoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|Получите _параметры_ объекта [MicrosoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md), которые указывают доступ из приложений Майкрософт к Microsoft 365 пользовательских данных в организации.|
|[Обновление microsoftApplicationDataAccessSettings](../api/microsoftapplicationdataaccesssettings-update.md)|[MicrosoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|Обновление параметров объекта [MicrosoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md), который указывает доступ из приложений Майкрософт к Microsoft 365 пользовательских данных в организации.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabledForAllMicrosoftApplications|Логический|Если установлено`true`, все пользователи в организации могут получить доступ в приложении Майкрософт к любым Microsoft 365 данным, к данным, к которые пользователь получил разрешение на доступ. Приложение Microsoft может быть приложением Microsoft 365 (например, Excel, Outlook) или Microsoft 365 приложением (например, Edge). Значение по умолчанию: `true`. <br> Этот доступ можно отключить для подмножество пользователей группы безопасности Azure AD, указав группу в свойстве **disabledForGroup** . <br> Если установлено`false`, все пользователи могут получить доступ к Microsoft 365 данным только в Microsoft 365 приложении.|
|disabledForGroup|String|ID группы безопасности Azure Active Directory Azure AD, для которой участникам разрешен доступ к данным Microsoft 365 с помощью только Microsoft 365 приложений, но не других приложений Майкрософт, таких как Edge. <br> Это применимо только в том случае, если **установлено для isEnabledForAllMicrosoftApplications** `true`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": "Boolean",
  "disabledForGroup": "String"
}
```
