---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b785f37676ac7f5651669c682c02126ffb36ff82
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609649"
---
# <a name="usersettings-resource-type"></a>Тип ресурса userSettings

Пространство имен: microsoft.graph

Параметры текущего пользователя для поиска контента.

Наследуется от [entity](entity.md). Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).

Этот ресурс поддерживает:

- Проверку участия пользователя и организации пользователя в поиске содержимого.
- Включение и отключение поиска содержимого для конкретных пользователей. При этом также отключаются документы в Office Delve.

> [!NOTE]
> Эта конечная точка работает только с пользователями. Вы не можете использовать эту конечную точку с контактами.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Получение параметров пользователя и организации. |
|[Обновление параметров пользователя](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ к API [trending](/graph/api/resources/insights-trending) пользователя отключен. Если задано значение true, документы в Office Delve пользователя отключены. Установка значения true влияет на релевантность содержимого, отображаемого в Microsoft 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](/graph/api/resources/insights-trending). Если задано значение true, у организации отсутствует доступ к Office Delve. Это влияет на релевантность содержимого, отображаемого в Microsoft 365 для всей организации, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|
|id|String|Уникальный идентификатор параметра пользователя. Только для чтения. Наследуется от [сущности](entity.md).|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```

