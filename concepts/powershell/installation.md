---
title: Установка пакета SDK PowerShell для Microsoft Graph
description: Содержит инструкции по установке пакета SDK PowerShell для Microsoft Graph.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 245cf03c8edf04a43c563bd19832eb0a35cf7cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193713"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Установка пакета SDK PowerShell для Microsoft Graph

Пакет SDK Microsoft Graph PowerShell опубликован в [коллекции PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph). Вы можете установить пакет SDK в PowerShell Core или Windows PowerShell с помощью следующей команды.

```powershell
Install-Module Microsoft.Graph
```

При необходимости вы можете изменить область установки по умолчанию с помощью `-Scope` параметра. Для этого требуются разрешения администратора.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> Установка пакета SDK в одной версии PowerShell не устанавливает ее для другого. Не забудьте выполнить команду установки в той версии PowerShell, в которой вы планируете ее использовать.

## <a name="verify-installation"></a>Проверка установки

После завершения установки можно проверить установленную версию с помощью следующей команды.

```powershell
Get-InstalledModule Microsoft.Graph
```

Версия в выходных данных должна отличаться от последней версии, опубликованной в галерее PowerShell. Теперь вы готовы использовать пакет SDK.

> [!div class="nextstepaction"]
> [Начало работы с пакетом SDK PowerShell для Microsoft Graph](get-started.md)

## <a name="updating-the-sdk"></a>Обновление пакета SDK

Вы можете обновить пакет SDK и все его зависимости с помощью следующей команды.

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>Удаление пакета SDK

Сначала удалите основной модуль с помощью следующей команды.

```powershell
Uninstall-Module Microsoft.Graph
```

Затем удалите все модули зависимости, выполнив указанные ниже команды.

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>Предоставление отзывов

Мы ждем отзывов! Сообщите о любой обратной связи или сообщите о проблемах в [репозитории GitHub SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).
