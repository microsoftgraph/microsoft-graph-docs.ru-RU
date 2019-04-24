---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462251"
---
#<a name="teamsappinstalledstate-enum-type"></a>тип перечисления Теамсаппинсталледстате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние установки [teamsApp](teamsapp.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Нотинсталлед|нуль|Приложение не установлено в группу.|
|устанавлива|1,1|Приложение устанавливается обычным образом.|
|Инсталледандхидден|2|Приложение установлено, но скрыто в представлении.|
|Инсталледандперманент|4|Приложение устанавливается без возможности восстановления и не может быть удалено.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
