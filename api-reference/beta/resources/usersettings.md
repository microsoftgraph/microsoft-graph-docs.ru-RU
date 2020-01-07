---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f3f04bc1c9432b2f46e440e1966ac65e310ec0d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951953"
---
# <a name="usersettings-resource-type"></a>Тип ресурса userSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры текущего пользователя для поиска контента. Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).

Этот ресурс поддерживает:

- Проверку участия пользователя и организации пользователя в поиске содержимого.
- Включение и отключение поиска содержимого для конкретных пользователей. При этом также отключаются документы в Office Delve.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Получение параметров пользователя и организации. |
|[Обновление параметров пользователя](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен. Если задано значение true, документы в Office Delve пользователя отключены. Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md). Если задано значение true, у организации отсутствует доступ к Office Delve. Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="relationships"></a>Отношения

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|шифтпреференцес|[шифтпреференцес](shiftpreferences.md)| Настройки смены для пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
