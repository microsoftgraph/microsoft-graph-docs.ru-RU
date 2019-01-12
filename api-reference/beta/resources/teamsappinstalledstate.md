---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937175"
---
#<a name="teamsappinstalledstate-enum-type"></a>Тип перечисления teamsAppInstalledState

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает текущее состояние установки [teamsApp](teamsapp.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|notInstalled|0|Приложение не установлено в группу.|
|установлен|1|Приложение устанавливается в обычном режиме.|
|installedAndHidden|2|Приложение установлен, но скрыты.|
|installedAndPermanent|3|Приложение устанавливается без возможности восстановления и не могут быть удалены.|
