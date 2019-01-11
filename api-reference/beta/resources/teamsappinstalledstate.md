---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847574"
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
