---
title: Установка пакета SDK Microsoft Graph PowerShell
description: Содержит инструкции по установке пакета SDK Microsoft Graph PowerShell.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 80086e4879ce9acb547e060c45891bd58dc602bf
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883390"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка пакета SDK Microsoft Graph PowerShell

> [!NOTE]
> При установке основного модуля пакета SDK будут устанавливаться все 38 подмножеов. Рассмотрите возможность установки только необходимых модулей, включая `Microsoft.Graph.Authentication`. Для списка доступных модулей Microsoft Graph используйте следующую команду.
>
> ```powershell
> Find-Module Microsoft.Graph*
> ```

Пакет SDK Microsoft Graph PowerShell публикуется [на коллекция PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph) Пакет SDK можно установить в PowerShell Core или Windows PowerShell с помощью следующей команды.

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

При необходимости можно изменить область установки с помощью параметра `-Scope` . Для этого требуются разрешения администратора.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> При установке пакета SDK в одной версии PowerShell он не устанавливается для другой. Обязательно выполните команду установки в версии PowerShell, в которой она будет использоваться.

## <a name="supported-powershell-versions"></a>Поддерживаемые версии PowerShell

PowerShell 7 и более поздних версий — это рекомендуемая версия PowerShell для использования с пакетом SDK Microsoft Graph PowerShell на всех платформах. Нет дополнительных предварительных условий для использования пакета SDK с PowerShell 7 или более поздней версии.

Чтобы использовать пакет SDK Microsoft Graph PowerShell с Windows PowerShell, необходимо выполнить следующие предварительные требования.

- Обновление до [PowerShell 5.1 или более поздней версии](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)
- Установка [платформа .NET Framework 4.7.2 или более поздней версии](/dotnet/framework/install/)
- Обновление **PowerShellGet до** последней версии с помощью `Install-Module PowerShellGet -Force`

## <a name="verify-installation"></a>Проверка установки

После завершения установки можно проверить установленную версию с помощью следующей команды.

```powershell
Get-InstalledModule Microsoft.Graph
```

Версия в выходных данных должна соответствовать последней версии, опубликованной на коллекция PowerShell. Теперь вы готовы использовать пакет SDK.

> [!div class="nextstepaction"]
> [Начало работы с пакетом SDK Microsoft Graph PowerShell](get-started.md)

## <a name="updating-the-sdk"></a>Обновление пакета SDK

Пакет SDK и все его зависимости можно обновить с помощью следующей команды.

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>Удаление пакета SDK

Сначала выполните следующую команду, чтобы удалить основной модуль.

```powershell
Uninstall-Module Microsoft.Graph
```

Затем удалите все модули зависимостей, выполнив следующие команды.

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>Предоставление отзывов

Мы будем рады получить отзыв! Предоставьте отзыв или сообщите о любых проблемах в [репозитории GitHub пакета SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).
