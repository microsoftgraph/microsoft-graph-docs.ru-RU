---
title: Members
description: Описывает текущее состояние установки teamsApp.
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316795"
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
