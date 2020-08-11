---
title: Отчеты об использовании приложений Microsoft 365
description: Используйте отчеты об использовании приложений Microsoft 365 для получения ценных сведений об использовании приложений Microsoft 365 в вашей организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f9b83608f3a5859e696c4ea2c52e22e35d291fce
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630472"
---
# <a name="microsoft-365-apps-usage-reports"></a>Отчеты об использовании приложений Microsoft 365

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты об использовании приложений Microsoft 365 для получения ценных сведений об использовании приложений Microsoft 365 в вашей организации.

## <a name="methods"></a>Методы

| Метод                                                                        | Возвращаемый тип                                    | Описание                                                |
| :---------------------------------------------------------------------------- | :--------------------------------------------- | :--------------------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getm365appuserdetail.md)                  | [report](../resources/intune-shared-report.md) | Получение сведений об использовании приложений Microsoft 365 пользователем. |
| [Получение количества пользователей](../api/reportroot-getm365appusercounts.md)                  | [report](../resources/intune-shared-report.md) | Получение числа ежедневных уникальных пользователей по приложению.               |
| [Получение числа пользователей платформы](../api/reportroot-getm365appplatformusercounts.md) | [report](../resources/intune-shared-report.md) | Получение числа ежедневных уникальных пользователей по платформе.          |
