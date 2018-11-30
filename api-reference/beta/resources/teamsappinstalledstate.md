---
title: Элементы
description: Описывает текущее состояние установки teamsApp.
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080672"
---
#<a name="teamsappinstalledstate-enum-type"></a>Тип перечисления teamsAppInstalledState

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает текущее состояние установки [teamsApp](teamsapp.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Description |
|:---------------|:--------|:----------|
|notInstalled|0|Приложение не установлено в группу.|
|установлен|1|Приложение устанавливается в обычном режиме.|
|installedAndHidden|2|Приложение установлен, но скрыты.|
|installedAndPermanent|3|Приложение устанавливается без возможности восстановления и не могут быть удалены.|
