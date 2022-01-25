---
title: Установка SDK Graph Microsoft Graph PowerShell
description: Содержит инструкции по установке SDK Graph PowerShell.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 0337b4641f8c84e63c4c5e7eecf1da0f186dad0c
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201682"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка SDK Graph Microsoft Graph PowerShell

> [!NOTE]
> Установка основного модуля SDK установит все 38 модулей. Рассмотрим только установку необходимых модулей, в том числе `Microsoft.Graph.Authentication` . Для списка доступных модулей Microsoft Graph используйте следующую команду.
>
> ```powershell
> Find-Module Microsoft.Graph*
> ```

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

## <a name="supported-powershell-versions"></a>Поддерживаемые версии PowerShell

PowerShell 7 и более поздние версии PowerShell рекомендуется использовать с microsoft Graph PowerShell SDK на всех платформах. Нет дополнительных предпосылок для использования SDK с PowerShell 7 или более поздней.

Для использования SDK Microsoft Graph PowerShell с помощью Windows PowerShell.

- Обновление до [PowerShell 5.1 или более поздней](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)
- Установка [платформа .NET Framework 4.7.2 или более поздней](/dotnet/framework/install/)
- Обновление **PowerShellGet** до последней версии с помощью `Install-Module PowerShellGet -Force`

## <a name="verify-installation"></a>Проверка установки

После завершения установки можно проверить установленную версию следующей командой.

```powershell
Get-InstalledModule Microsoft.Graph
```

Версия в выходе должна соответствовать последней версии, опубликованной в Галерее PowerShell. Теперь вы готовы использовать SDK.

> [!div class="nextstepaction"]
> [Начало работы с пакетом SDK Microsoft Graph PowerShell](get-started.md)

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
