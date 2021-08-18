---
title: тип enum resultantAppStateDetail
description: Enum указывает дополнительные сведения о том, почему приложение имеет определенное состояние установки.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4b83040763f0b7b56c4a6e8979a06f3f945a39ed94dde254c042648f8fe349f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54250065"
---
# <a name="resultantappstatedetail-enum-type"></a>тип enum resultantAppStateDetail

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Enum указывает дополнительные сведения о том, почему приложение имеет определенное состояние установки.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noAdditionalDetails|0|Дополнительные сведения недоступны.|
|dependencyFailedToInstall|1 |Одна или несколько зависимостей приложения не удалось установить.|
|dependencyWithRequirementsNotMet|2|Одна или несколько зависимостей приложения имеют требования, которые не выполнены.|
|dependencyPendingReboot|3 |Для одной или более зависимостей приложения требуется перезагрузка устройства для завершения установки.|
|dependencyWithAutoInstallDisabled|4 |Одна или несколько зависимостей приложения настроены для автоматической установки.|
|iosAppStoreUpdateFailedToInstall|1000|Последняя версия приложения не обновлялась из более ранней версии.|
|vppAppHasUpdateAvailable|1001|Доступно обновление.|
|userRejectedUpdate|1002|Пользователь отклонил обновление приложения. |
|seeInstallErrorCode|2000|Приложение не удалось установить. Дополнительные сведения см. в свойстве кода ошибки.|
|autoInstallDisabled|3000|Приложение настроено на автоматическое установку.|
|managedAppNoLongerPresent|3001|Приложение управляется, но больше не устанавливается.|
|userRejectedInstall|3002|Пользователь отклонил установку приложения.|
|userIsNotLoggedIntoAppStore|3003|Чтобы установить приложение, пользователь должен войти в App Store.|
|seeUninstallErrorCode|4000|Приложение не удалось удалить. Дополнительные сведения см. в свойстве кода ошибки.|
|pendingReboot|5000|Устройство должно быть перезагружается для завершения установки приложения.|
|installingDependencies|5001|Устанавливается одна или несколько зависимостей приложения.|
|contentDownloaded|5002|Содержимое приложения было загружено на устройство.|
|powerShellScriptRequirementNotMet|-1013|Правило требования к сценарию PowerShell не соответствует|
|registryRequirementNotMet|-1012|Правило требования реестра не соответствует|
|fileSystemRequirementNotMet|-1011|Правило требования к системе файлов не соответствует|
|platformNotApplicable|-1006|Приложение не применимо к этой платформе. (например, android-приложение для IOS)|
|minimumCpuSpeedNotMet|-1005|Скорость ЦП на целевом устройстве меньше установленного минимума.|
|minimumLogicalProcessorCountNotMet|-1004|Количество логических процессоров на целевом устройстве меньше установленного минимума.|
|minimumPhysicalMemoryNotMet|-1003|Объем оперативной памяти на целевом устройстве меньше установленного минимума.|
|minimumOsVersionNotMet|-1002|Версия ОС на целевом устройстве меньше установленного минимума.|
|minimumDiskSpaceNotMet|-1001|Доступное пространство диска на целевом устройстве меньше установленного минимума.|
|processorArchitectureNotApplicable|-1000|Архитектура устройства (например, x86/amd64) не применима к приложению.|




