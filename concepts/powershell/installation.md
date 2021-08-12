---
title: Установка SDK Graph Microsoft Graph PowerShell
description: Содержит инструкции по установке SDK Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 9a23e9498920f329cca5d8eaaef6178c9291803ec9ede965f2fe7569e0b454c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149522"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка SDK Graph Microsoft Graph PowerShell

> [!NOTE]
> Установка основного модуля SDK установит все 38 модулей. Рассмотрим только установку необходимых модулей, в том числе `Microsoft.Graph.Authentication` .

SDK Graph Microsoft Graph PowerShell опубликован в [галерее PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph) Можно установить SDK в PowerShell Core или Windows PowerShell с помощью следующей команды.

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

Необязательно можно изменить область установки с помощью `-Scope` параметра. Для этого требуются разрешения администратора.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> Установка SDK в одной версии PowerShell не устанавливает его для другой. Не забудьте запустить команду установки в версии PowerShell, в которая вы собираетесь использовать ее.

## <a name="verify-installation"></a>Проверка установки

После завершения установки можно проверить установленную версию следующей командой.

```powershell
Get-InstalledModule Microsoft.Graph
```

Версия в выходе должна соответствовать последней версии, опубликованной в Галерее PowerShell. Теперь вы готовы использовать SDK.

> [!div class="nextstepaction"]
> [Начало работы с SDK Microsoft Graph PowerShell](get-started.md)

## <a name="updating-the-sdk"></a>Обновление SDK

Вы можете обновить SDK и все его зависимости с помощью следующей команды.

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>Uninstalling the SDK

Сначала используйте следующую команду, чтобы удалить основной модуль.

```powershell
Uninstall-Module Microsoft.Graph
```

Затем удалите все модули зависимостей, запуская следующие команды.

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>Предоставление отзывов

Мы приветствуем отзывы! Просьба предоставить любые отзывы или сообщить о проблемах в репозитории [SDK GitHub.](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)
