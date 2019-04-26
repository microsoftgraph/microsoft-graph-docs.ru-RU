---
title: Тип ресурса "Параметры"
description: 'Параметры текущего пользователя. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554270"
---
# <a name="settings-resource-type"></a>Тип ресурса "Параметры"

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры текущего пользователя. Чтобы узнать, как получить или обновить параметры пользователя, ознакомьтесь со [статьЕй получение параметров](../api/user-get-settings.md) и [Обновление параметров](../api/user-update-settings.md).

Этот ресурс поддерживает:

- Проверка того, участвует ли пользователь и пользователь в Организации для обнаружения контента.
- Отключение или Включение обнаружения контента для определенных пользователей. При этом также отключаются документы в Office delve.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/user-get-settings.md) |[settings](../resources/user-settings.md)| Получение параметров пользователя и Организации. |
|[Обновление параметров пользователя](../api/user-update-settings.md) |[settings](../resources/user-settings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Контрибутионтоконтентдисковеридисаблед|Логический|Если задано значение true, доступ представителя к API [трендов](insights-trending.md) пользователя отключен. Если задано значение true, документы в Office delve пользователя отключены. Если задано значение true, то релевантность содержимого, отображаемого в Office 365, например в разделе Рекомендуемые сайты в SharePoint Home и представление "Обнаружение" в OneDrive для бизнеса влияет. Пользователи могут управлять этим параметром в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|Контрибутионтоконтентдисковерясорганизатиондисаблед|Логический|Отражает [параметр уровня Организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) , контролирующий доступ делегата [](insights-trending.md) к API тенденций. Если задано значение true, Организация не имеет доступа к Office delve. Релевантность контента, отображаемого в Office 365, например в разделе Рекомендуемые сайты в SharePoint Home, а представление обнаружения в OneDrive для бизнеса влияет на всю организацию. Этот параметр доступен только для чтения и может быть изменен только администраторами в [центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
