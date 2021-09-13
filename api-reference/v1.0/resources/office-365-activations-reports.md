---
title: Microsoft 365 отчеты об активациях
description: Отчеты Microsoft 365 активации могут дать представление о том, какие пользователи активировали Microsoft 365 по крайней мере на одном устройстве. Эти отчеты предоставляют разбивку активаций Microsoft 365, Project и Visio Pro для Office 365, а также разбивку активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 44742cf11676e751700c4f97d4aa5789f6da0f0b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084253"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365 отчеты об активациях

Пространство имен: microsoft.graph

Отчеты Microsoft 365 активации могут дать представление о том, какие пользователи активировали Microsoft 365 по крайней мере на одном устройстве. Эти отчеты предоставляют разбивку активаций Microsoft 365, Project и Visio Pro для Office 365, а также разбивку активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.

> **Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft Office активаций.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | Сведения о пользователях, активировавших Microsoft 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток      | Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |

